---
layout: reference
title: checklist
---

<script>
$(document).ready(function() {
	// apply line-through CSS to checked SCs
	$('input:checkbox').live('click', function () {
			// access parent li, do whatever you want with it
			$(this).parent("li").toggleClass('checked');
	});    

	// check which levels you want to appear
	$('input:checkbox#levela').live('click', function () {
			// access parent li, do whatever you want with it
			$('.levela').toggleClass('hidden');
	});    

	$('input:checkbox#levelaa').live('click', function () {
			// access parent li, do whatever you want with it
			$('.levelaa').toggleClass('hidden');
	});

	$('input:checkbox#levelaaa').live('click', function () {
			// access parent li, do whatever you want with it
			$('.levelaaa').toggleClass('hidden');
	});

	//zebra stripe list items
	$('li:even').addClass('stripe');

	//make tap area bigger to check boxes in iOS
	$('label').each(function() {
		var $this = $(this);
		if($this.attr('for') !== undefined) {
			$this.bind('click', function() {
				$('#'+$this.attr('for')).focus();
			});
		}
		else {
			$this.bind('click', function() {
				$this.find('input,button,select,textarea').eq(0).focus();
			});
		}
	});
});
</script>

<table border="0" cellpadding="0" cellspacing="0">
   <tr>
	  <td valign="top">
		 <ul>
			<li><a target="_blank" href="http://www.w3.org/TR/UNDERSTANDING-WCAG20/text-equiv.html">1.1 Text Alternatives</a></li>
			<ul>
			   <label>
				  <li class="levela"><input name="1.1.1" type="checkbox" id="1.1.1" /><a target="_blank" href="http://www.w3.org/TR/UNDERSTANDING-WCAG20/text-equiv-all.html">1.1.1 Non-text Content A</a></li>
			   </label>
			</ul>
			<li><a target="_blank" href="http://www.w3.org/TR/UNDERSTANDING-WCAG20/media-equiv.html">1.2 Time-based Media</a></li>
			<ul>
			   <label>
				  <li class="levela"><input type="checkbox" /><a target="_blank" href="http://www.w3.org/TR/UNDERSTANDING-WCAG20/media-equiv-av-only-alt.html">1.2.1 Audio-only and Video-only (Prerecorded) A</a></li>
			   </label>
			   <label>
				  <li class="levela"><input type="checkbox" /><a target="_blank" href="http://www.w3.org/TR/UNDERSTANDING-WCAG20/media-equiv-captions.html">1.2.2 Captions (Prerecorded) A</a></li>
			   </label>
			   <label>
				  <li class="levela"><input type="checkbox" /><a target="_blank" href="http://www.w3.org/TR/UNDERSTANDING-WCAG20/media-equiv-audio-desc.html">1.2.3 Audio Description or Media Alternative (Prerecorded) A</a></li>
			   </label>
			   <label>
				  <li class="levelaa"><input type="checkbox" /><a target="_blank" href="http://www.w3.org/TR/UNDERSTANDING-WCAG20/media-equiv-real-time-captions.html">1.2.4 Captions (Live) AA</a></li>
			   </label>
			   <label>
				  <li class="levelaa"><input type="checkbox" /><a target="_blank" href="http://www.w3.org/TR/UNDERSTANDING-WCAG20/media-equiv-audio-desc-only.html">1.2.5 Audio Description (Prerecorded) AA</a></li>
			   </label>
			   <label>
				  <li class="levelaaa"><input type="checkbox" /><a target="_blank" href="http://www.w3.org/TR/UNDERSTANDING-WCAG20/media-equiv-sign.html">1.2.6 Sign Language (Prerecorded) AAA</a></li>
			   </label>
			   <label>
				  <li class="levelaaa"><input type="checkbox" /><a target="_blank" href="http://www.w3.org/TR/UNDERSTANDING-WCAG20/media-equiv-extended-ad.html">1.2.7 Extended Audio Description (Prerecorded) AAA</a></li>
			   </label>
			   <label>
				  <li class="levelaaa"><input type="checkbox" /><a target="_blank" href="http://www.w3.org/TR/UNDERSTANDING-WCAG20/media-equiv-text-doc.html">1.2.8 Media Alternative (Prerecorded) AAA</a></li>
			   </label>
			   <label>
				  <li class="levelaaa"><input type="checkbox" /><a target="_blank" href="http://www.w3.org/TR/UNDERSTANDING-WCAG20/media-equiv-live-audio-only.html">1.2.9 Audio-only (Live) AAA</a></li>
			   </label>
			</ul>
			<li><a target="_blank" href="http://www.w3.org/TR/UNDERSTANDING-WCAG20/content-structure-separation.html">1.3 Adaptable</a></li>
			<ul>
			   <label>
				  <li class="levela"><input type="checkbox" /><a target="_blank" href="http://www.w3.org/TR/UNDERSTANDING-WCAG20/content-structure-separation-programmatic.html">1.3.1 Info and Relationships A</a></li>
			   </label>
			   <label>
				  <li class="levela"><input type="checkbox" /><a target="_blank" href="http://www.w3.org/TR/UNDERSTANDING-WCAG20/content-structure-separation-sequence.html">1.3.2 Meaningful Sequence A</a></li>
			   </label>
			   <label>
				  <li class="levela"><input type="checkbox" /><a target="_blank" href="http://www.w3.org/TR/UNDERSTANDING-WCAG20/content-structure-separation-understanding.html">1.3.3 Sensory Characteristics A</a></li>
			   </label>
			</ul>
			<li><a target="_blank" href="http://www.w3.org/TR/UNDERSTANDING-WCAG20/visual-audio-contrast.html">1.4 Distinguishable</a></li>
			<ul>
			   <label>
				  <li class="levela"><input type="checkbox" /><a target="_blank" href="http://www.w3.org/TR/UNDERSTANDING-WCAG20/visual-audio-contrast-without-color.html">1.4.1 Use of Color A</a></li>
			   </label>
			   <label>
				  <li class="levela"><input type="checkbox" /><a target="_blank" href="http://www.w3.org/TR/UNDERSTANDING-WCAG20/visual-audio-contrast-dis-audio.html">1.4.2 Audio Control A</a></li>
			   </label>
			   <label>
				  <li class="levelaa"><input type="checkbox" /><a target="_blank" href="http://www.w3.org/TR/UNDERSTANDING-WCAG20/visual-audio-contrast-contrast.html">1.4.3 Contrast (Minimum) AA</a></li>
			   </label>
			   <label>
				  <li class="levelaa"><input type="checkbox" /><a target="_blank" href="http://www.w3.org/TR/UNDERSTANDING-WCAG20/visual-audio-contrast-scale.html">1.4.4 Resize Text AA</a></li>
			   </label>
			   <label>
				  <li class="levelaa"><input type="checkbox" /><a target="_blank" href="http://www.w3.org/TR/UNDERSTANDING-WCAG20/visual-audio-contrast-text-presentation.html">1.4.5 Images of Text AA</a></li>
			   </label>
			   <label>
				  <li class="levelaaa"><input type="checkbox" /><a target="_blank" href="http://www.w3.org/TR/UNDERSTANDING-WCAG20/visual-audio-contrast7.html">1.4.6 Contrast (Enhanced) AAA</a></li>
			   </label>
			   <label>
				  <li class="levelaaa"><input type="checkbox" /><a target="_blank" href="http://www.w3.org/TR/UNDERSTANDING-WCAG20/visual-audio-contrast-noaudio.html">1.4.7 Low or No Background Audio AAA</a></li>
			   </label>
			   <label>
				  <li class="levelaaa"><input type="checkbox" /><a target="_blank" href="http://www.w3.org/TR/UNDERSTANDING-WCAG20/visual-audio-contrast-visual-presentation.html">1.4.8 Visual Presentation AAA</a></li>
			   </label>
			   <label>
				  <li class="levelaaa"><input type="checkbox" /><a target="_blank" href="http://www.w3.org/TR/UNDERSTANDING-WCAG20/visual-audio-contrast-text-images.html">1.4.9 Images of Text (No Exception) AAA</a></li>
			   </label>
			</ul>
			<li><a target="_blank" href="http://www.w3.org/TR/UNDERSTANDING-WCAG20/keyboard-operation.html">2.1 Keyboard Accessible</a></li>
			<ul>
			   <label>
				  <li class="levela"><input type="checkbox" /><a target="_blank" href="http://www.w3.org/TR/UNDERSTANDING-WCAG20/keyboard-operation-keyboard-operable.html">2.1.1 Keyboard A</a></li>
			   </label>
			   <label>
				  <li class="levela"><input type="checkbox" /><a target="_blank" href="http://www.w3.org/TR/UNDERSTANDING-WCAG20/keyboard-operation-trapping.html">2.1.2 No Keyboard Trap A</a></li>
			   </label>
			   <label>
				  <li class="levelaaa"><input type="checkbox" /><a target="_blank" href="http://www.w3.org/TR/UNDERSTANDING-WCAG20/keyboard-operation-all-funcs.html">2.1.3 Keyboard (No Exception) AAA</a></li>
			   </label>
			</ul>
			<li><a target="_blank" href="http://www.w3.org/TR/UNDERSTANDING-WCAG20/time-limits.html">2.2 Enough Time</a></li>
			<ul>
			   <label>
				  <li class="levela"><input type="checkbox" /><a target="_blank" href="http://www.w3.org/TR/UNDERSTANDING-WCAG20/time-limits-required-behaviors.html">2.2.1 Timing Adjustable A</a></li>
			   </label>
			   <label>
				  <li class="levela"><input type="checkbox" /><a target="_blank" href="http://www.w3.org/TR/UNDERSTANDING-WCAG20/time-limits-pause.html">2.2.2 Pause, Stop, Hide A</a></li>
			   </label>
			   <label>
				  <li class="levelaaa"><input type="checkbox" /><a target="_blank" href="http://www.w3.org/TR/UNDERSTANDING-WCAG20/time-limits-no-exceptions.html">2.2.3 No Timing AAA</a></li>
			   </label>
			   <label>
				  <li class="levelaaa"><input type="checkbox" /><a target="_blank" href="http://www.w3.org/TR/UNDERSTANDING-WCAG20/time-limits-postponed.html">2.2.4 Interruptions AAA</a></li>
			   </label>
			   <label>
				  <li class="levelaaa"><input type="checkbox" /><a target="_blank" href="http://www.w3.org/TR/UNDERSTANDING-WCAG20/time-limits-server-timeout.html">2.2.5 Re-authenticating AAA</a></li>
			   </label>
			</ul>
		 </ul>
	  </td>
	  <td valign="top">
		 <ul>
			<li><a target="_blank" href="http://www.w3.org/TR/UNDERSTANDING-WCAG20/seizure.html">2.3 Seizures</a></li>
			<ul>
			   <label>
				  <li class="levela"><input type="checkbox" /><a target="_blank" href="http://www.w3.org/TR/UNDERSTANDING-WCAG20/seizure-does-not-violate.html">2.3.1 Three Flashes or Below Threshold A</a></li>
			   </label>
			   <label>
				  <li class="levelaaa"><input type="checkbox" /><a target="_blank" href="http://www.w3.org/TR/UNDERSTANDING-WCAG20/seizure-three-times.html">2.3.2 Three Flashes AAA</a></li>
			   </label>
			</ul>
			<li><a target="_blank" href="http://www.w3.org/TR/UNDERSTANDING-WCAG20/navigation-mechanisms.html">2.4 Navigable</a></li>
			<ul>
			   <label>
				  <li class="levela"><input type="checkbox" /><a target="_blank" href="http://www.w3.org/TR/UNDERSTANDING-WCAG20/navigation-mechanisms-skip.html">2.4.1 Bypass Blocks A</a></li>
			   </label>
			   <label>
				  <li class="levela"><input type="checkbox" /><a target="_blank" href="http://www.w3.org/TR/UNDERSTANDING-WCAG20/navigation-mechanisms-title.html">2.4.2 Page Titled A</a></li>
			   </label>
			   <label>
				  <li class="levela"><input type="checkbox" /><a target="_blank" href="http://www.w3.org/TR/UNDERSTANDING-WCAG20/navigation-mechanisms-focus-order.html">2.4.3 Focus Order A</a></li>
			   </label>
			   <label>
				  <li class="levela"><input type="checkbox" /><a target="_blank" href="http://www.w3.org/TR/UNDERSTANDING-WCAG20/navigation-mechanisms-refs.html">2.4.4 Link Purpose (In Context) A</a></li>
			   </label>
			   <label>
				  <li class="levelaa"><input type="checkbox" /><a target="_blank" href="http://www.w3.org/TR/UNDERSTANDING-WCAG20/navigation-mechanisms-mult-loc.html">2.4.5 Multiple Ways AA</a></li>
			   </label>
			   <label>
				  <li class="levelaa"><input type="checkbox" /><a target="_blank" href="http://www.w3.org/TR/UNDERSTANDING-WCAG20/navigation-mechanisms-descriptive.html">2.4.6 Headings and Labels AA</a></li>
			   </label>
			   <label>
				  <li class="levelaa"><input type="checkbox" /><a target="_blank" href="http://www.w3.org/TR/UNDERSTANDING-WCAG20/navigation-mechanisms-focus-visible.html">2.4.7 Focus Visible AA</a></li>
			   </label>
			   <label>
				  <li class="levelaaa"><input type="checkbox" /><a target="_blank" href="http://www.w3.org/TR/UNDERSTANDING-WCAG20/navigation-mechanisms-location.html">2.4.8 Location AAA</a></li>
			   </label>
			   <label>
				  <li class="levelaaa"><input type="checkbox" /><a target="_blank" href="http://www.w3.org/TR/UNDERSTANDING-WCAG20/navigation-mechanisms-link.html">2.4.9 Link Purpose (Link Only) AAA</a></li>
			   </label>
			   <label>
				  <li class="levelaaa"><input type="checkbox" /><a target="_blank" href="http://www.w3.org/TR/UNDERSTANDING-WCAG20/navigation-mechanisms-headings.html">2.4.10 Section Headings AAA</a></li>
			   </label>
			</ul>
			<li><a target="_blank" href="http://www.w3.org/TR/UNDERSTANDING-WCAG20/meaning.html">3.1 Readable</a></li>
			<ul>
			   <label>
				  <li class="levela"><input type="checkbox" /><a target="_blank" href="http://www.w3.org/TR/UNDERSTANDING-WCAG20/meaning-doc-lang-id.html">3.1.1 Language of Page A</a></li>
			   </label>
			   <label>
				  <li class="levelaa"><input type="checkbox" /><a target="_blank" href="http://www.w3.org/TR/UNDERSTANDING-WCAG20/meaning-other-lang-id.html">3.1.2 Language of Parts AA</a></li>
			   </label>
			   <label>
				  <li class="levelaaa"><input type="checkbox" /><a target="_blank" href="http://www.w3.org/TR/UNDERSTANDING-WCAG20/meaning-idioms.html">3.1.3 Unusual Words AAA</a></li>
			   </label>
			   <label>
				  <li class="levelaaa"><input type="checkbox" /><a target="_blank" href="http://www.w3.org/TR/UNDERSTANDING-WCAG20/meaning-located.html">3.1.4 Abbreviations AAA</a></li>
			   </label>
			   <label>
				  <li class="levelaaa"><input type="checkbox" /><a target="_blank" href="http://www.w3.org/TR/UNDERSTANDING-WCAG20/meaning-supplements.html">3.1.5 Reading Level AAA</a></li>
			   </label>
			   <label>
				  <li class="levelaaa"><input type="checkbox" /><a target="_blank" href="http://www.w3.org/TR/UNDERSTANDING-WCAG20/meaning-pronunciation.html">3.1.6 Pronunciation AAA</a></li>
			   </label>
			</ul>
			<li><a target="_blank" href="http://www.w3.org/TR/UNDERSTANDING-WCAG20/consistent-behavior.html">3.2 Predictable</a></li>
			<ul>
			   <label>
				  <li class="levela"><input type="checkbox" /><a target="_blank" href="http://www.w3.org/TR/UNDERSTANDING-WCAG20/consistent-behavior-receive-focus.html">3.2.1 On Focus A</a></li>
			   </label>
			   <label>
				  <li class="levela"><input type="checkbox" /><a target="_blank" href="http://www.w3.org/TR/UNDERSTANDING-WCAG20/consistent-behavior-unpredictable-change.html">3.2.2 On Input A</a></li>
			   </label>
			   <label>
				  <li class="levelaa"><input type="checkbox" /><a target="_blank" href="http://www.w3.org/TR/UNDERSTANDING-WCAG20/consistent-behavior-consistent-locations.html">3.2.3 Consistent Navigation AA</a></li>
			   </label>
			   <label>
				  <li class="levelaa"><input type="checkbox" /><a target="_blank" href="http://www.w3.org/TR/UNDERSTANDING-WCAG20/consistent-behavior-consistent-functionality.html">3.2.4 Consistent Identification AA</a></li>
			   </label>
			   <label>
				  <li class="levelaaa"><input type="checkbox" /><a target="_blank" href="http://www.w3.org/TR/UNDERSTANDING-WCAG20/consistent-behavior-no-extreme-changes-context.html">3.2.5 Change on Request AAA</a></li>
			   </label>
			</ul>
			<li><a target="_blank" href="http://www.w3.org/TR/UNDERSTANDING-WCAG20/minimize-error.html">3.3 Input Assistance</a></li>
			<ul>
			   <label>
				  <li class="levela"><input type="checkbox" /><a target="_blank" href="http://www.w3.org/TR/UNDERSTANDING-WCAG20/minimize-error-identified.html">3.3.1 Error Identification A</a></li>
			   </label>
			   <label>
				  <li class="levela"><input type="checkbox" /><a target="_blank" href="http://www.w3.org/TR/UNDERSTANDING-WCAG20/minimize-error-cues.html">3.3.2 Labels or Instructions A</a></li>
			   </label>
			   <label>
				  <li class="levelaa"><input type="checkbox" /><a target="_blank" href="http://www.w3.org/TR/UNDERSTANDING-WCAG20/minimize-error-suggestions.html">3.3.3 Error Suggestion AA</a></li>
			   </label>
			   <label>
				  <li class="levelaa"><input type="checkbox" /><a target="_blank" href="http://www.w3.org/TR/UNDERSTANDING-WCAG20/minimize-error-reversible.html">3.3.4 Error Prevention (Legal, Financial, Data) AA</a></li>
			   </label>
			   <label>
				  <li class="levelaaa"><input type="checkbox" /><a target="_blank" href="http://www.w3.org/TR/UNDERSTANDING-WCAG20/minimize-error-context-help.html">3.3.5 Help AAA</a></li>
			   </label>
			   <label>
				  <li class="levelaaa"><input type="checkbox" /><a target="_blank" href="http://www.w3.org/TR/UNDERSTANDING-WCAG20/minimize-error-reversible-all.html">3.3.6 Error Prevention (All) AAA</a></li>
			   </label>
			</ul>
			<li><a target="_blank" href="http://www.w3.org/TR/UNDERSTANDING-WCAG20/ensure-compat.html">4.1 Compatible</a></li>
			<ul>
			   <label>
				  <li class="levela"><input type="checkbox" /><a target="_blank" href="http://www.w3.org/TR/UNDERSTANDING-WCAG20/ensure-compat-parses.html">4.1.1 Parsing A</a></li>
			   </label>
			   <label>
				  <li class="levela"><input type="checkbox" /><a target="_blank" href="http://www.w3.org/TR/UNDERSTANDING-WCAG20/ensure-compat-rsv.html">4.1.2 Name, Role, Value A</a></li>
			   </label>
			</ul>
		 </ul>
	  </td>
   </tr>
</table>
		
<label><input type="checkbox" id="levela" checked />Level A</label>
<label><input type="checkbox" id="levelaa" checked />Level AA</label>
<label><input type="checkbox" id="levelaaa" checked />Level AAA</label>
